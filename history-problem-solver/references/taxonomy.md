# 问题分类表

版本：0.2。沿用原类别与标签 ID。供案例标注与按问题检索使用，不是人格分类或穷尽现实问题的理论。

## 分类之前先澄清阶段目标

人生方向问题中，先理解用户想增加、减少与保留的体验，再把它转为待决问题。安稳、创业、阶段收入、家庭责任或创造等是可重叠的目标线索，不新增为人格类别，也不因为用户选了某目标就自动检索某位历史人物。

目标暂不清楚时，先进行简短引导；已有明确目标时直接使用。案例的历史目标也要标明是史书记述还是分析假说，不用人物后来的结局反推其起初志向。

## 六个主类别

| 稳定 ID | 类别 | 需要决定什么 | 优先检查的变量 | 分类边界 |
|---|---|---|---|---|
| cooperation_trust | 合作与信任 | 是否合作、继续信任或设置边界 | integrity、competence、incentives、information_quality、exit_options | 核心是可靠性与合作条件；仅安排职责转向 organization_people |
| stay_leave | 去留与选择 | 留下、转换、继续投入还是退出 | alternatives、exit_options、switching_cost、sunk_cost、reversibility | 核心是路径选择；主要纠结行动日期则用 timing |
| timing | 时机把握 | 现在行动、等待还是分阶段推进 | time_window、readiness、information_quality、feedback_speed、option_value | 等待本身必须有成本和收益，不能只赞美耐心 |
| risk_uncertainty | 风险与不确定性 | 是否承担不确定后果、投入多少 | downside、uncertainty、resources、reversibility、option_value | 聚焦损失承受力与信息条件，不以“胆大”替代分析 |
| organization_people | 组织与用人 | 如何选人、授权、分工与建立反馈 | competence、accountability、incentives、power_balance、feedback_speed | 聚焦组织机制；道德品质或合作底线问题可兼标 cooperation_trust |
| competition_negotiation | 竞争与谈判 | 如何协商、竞争、结盟与达成可接受结果 | alternatives、power_balance、incentives、information_quality、dependencies | 先判断是否存在合作空间，不把所有关系都当零和博弈 |

## 标注与检索顺序

1. 先写出具体的待决问题，再选择一个 `primary_category`，必要时添加零至两个 `secondary_categories`。
2. 选三至六个最能区分案例的 `tags`。标签名称取自下表，优先变量而非人物或朝代；人物、时间另有字段。
3. 检索时先看待决问题与主类别，再看关键变量的机制和方向，最后核对结果与类比限制。不能仅凭标签重合认定适用。
4. 为关键变量记录实际取值或证据；“都有 integrity 标签”不足以解释一个成功、一个失败。
5. 类别不适配时，将 `primary_category` 设为 `unmapped`，在 `classification_note` 写明原因。`unmapped` 是待归类状态，不是第七个万能类别；可以不使用历史分析。
6. 新标签先写进说明供讨论，不临时创造同义 ID。调整分类时保留旧 ID 的映射，避免已有案例失去索引。

## 受控标签与关键问题

| 标签 ID | 含义 | 现实中检查什么 |
|---|---|---|
| integrity | 诚信与行为可靠性 | 哪些可核实的承诺被兑现或违背，是否存在持续模式？ |
| competence | 任务能力 | 是否有与当前任务直接相关的表现证据？ |
| incentives | 激励与利益 | 谁获得收益、谁承担成本，利益是否冲突？ |
| information_quality | 信息质量 | 信息从何而来，有无独立核验和盲点？ |
| alternatives | 替代选项 | 不接受当前方案还能做什么？ |
| exit_options | 退出空间 | 能否退出，退出需要谁同意、付出什么？ |
| switching_cost | 转换成本 | 转换路径需要重新投入哪些资源？ |
| sunk_cost | 沉没成本 | 已不可收回的投入是否干扰未来判断？ |
| reversibility | 可逆性 | 哪些后果可以撤销，哪些不可恢复？ |
| time_window | 时间窗口 | 截止日期与机会消失是否有实际依据？ |
| readiness | 行动条件 | 当前是否具备必要资源与能力？ |
| feedback_speed | 反馈速度 | 多久能看到有效信号，信号是否可解释？ |
| option_value | 保留选择的价值 | 小步行动或等待能否保留后续选项？ |
| downside | 不利后果 | 最坏的可信情景是什么，谁承受得起？ |
| uncertainty | 不确定性 | 哪些未知可调查，哪些只能接受？ |
| resources | 资源约束 | 时间、精力、资金和支持的上限是什么？ |
| accountability | 权责与问责 | 责任、决策权、复核与申诉渠道是否清楚？ |
| power_balance | 权力与议价能力 | 各方能决定什么，能否拒绝或争取外部支持？ |
| dependencies | 相互依赖 | 哪个环节或参与方失效会影响整体？ |
| value_conflict | 价值冲突 | 哪些目标不能同时实现，由谁作价值选择？ |
| boundaries | 个人或合作边界 | 可接受与不可接受的行为分别是什么？ |
| learning_feedback | 学习与纠错 | 错误在哪里，练习是否得到有效反馈？ |

## 场景与类别不要混为一谈

“学习”“家庭”“工作”“个人成长”属于生活场景，可写入案例的 `modern_problem_examples`。它们不自动决定问题类别。例如：

- “复习两个月仍不会，是否更换方法”：通常先检查练习与反馈，可能用 stay_leave + learning_feedback；没有贴切史例就直接分析学习过程。
- “能力强但曾失信的人邀请合作”：cooperation_trust 为主，结合 integrity、competence、exit_options 等变量。
- “是否再等一个月谈加薪”：若核心是条件成熟度，用 timing；若核心是筹码与协商，用 competition_negotiation。
- “伴侣骗过我一次”：可以分析信任与边界，但不能自动推断其危险性，或套用君臣背叛叙事。
- “买哪种颜色的手机”：通常无需本技能的分类和历史检索。

对无法归类的意义、身份或道德困境，先尊重用户的表达；不要为了填表把它们重写成竞争、收益或管理问题。
