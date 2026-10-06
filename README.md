# 以史为鉴

**用中国历史案例，帮你分析去留、合作与时机选择，形成可验证的下一步。**

`history-problem-solver` 是一个结合中国历史决策结构与现代问题解决方法的 AI agent skill。它先厘清你的目标，再检查古今类比是否成立，比较行动路径，并说明何时需要重新判断。历史提供参照，现实证据决定行动。

History-informed decision support with Chinese historical cases and modern problem-solving methods.

[GitHub 仓库](https://github.com/Jetting-L/yi-shi-wei-jian) · [skills.sh 技能目录](https://skills.sh/jetting-l/yi-shi-wei-jian/history-problem-solver)

## 快速试用（Codex）

需要已安装 Node.js（提供 `npx`）和可使用本地技能的 Codex。在你希望使用技能的项目目录中运行：

```bash
npx --yes skills add Jetting-L/yi-shi-wei-jian --skill history-problem-solver --agent codex --copy --yes
```

命令将技能安装到当前项目的 `.agents/skills/history-problem-solver/`，属于项目级安装。打开该项目后，在 Codex 中输入 `$history-problem-solver` 调用；如果未出现，重新启动 Codex。

复制以下提问，替换方括号内容：

```text
请用 $history-problem-solver 帮我分析这个困境：
我正在考虑：[具体决定]。
我希望下一阶段：[想获得或保留的东西]。
已知事实与限制：[时间、资源、相关人的实际行为]。
目前的选项：[已有选项；没有也可以说明]。
请先澄清会影响判断的关键问题，再按需要核对历史类比，
比较路径，给出一个可执行的下一步和重新判断的条件。
```

目标还不清楚时，也可以直接说“我不知道下一阶段想要什么”，先从目标澄清开始。

## 适合什么问题

- **去留选择**：继续投入、调整参与方式，还是退出？各条路径如何服务你的阶段目标？
- **合作与信任**：承诺与行动是否一致？激励、责任、权限和退出空间怎样影响合作？
- **时机与风险**：现在行动、先做小规模试验，还是等待关键证据？什么信号会改变判断？

历史案例用于提出可检验的结构问题，不强行把古代人物或结局套到现代处境。没有贴切案例时，继续现实分析。

想先了解对话方式，可阅读已有的[完整对话示范](history-problem-solver/references/examples/goal_to_action.md)。其中用户、数字和结果均为虚构，不是试用反馈或效果证明。

## 其他使用方式与安装说明

技能入口为 [SKILL.md](history-problem-solver/SKILL.md)。也可从公开仓库下载完整 `history-problem-solver/` 目录，在支持本地技能的环境中使用；只复制 `SKILL.md` 会缺少按需加载的案例与方法卡。

如果当前助手能访问本仓库文件，也可直接要求它按 `SKILL.md` 流程、按需读取资源。这种方式不等于已安装或已验证该助手的技能兼容性。

安装命令来自第三方 [skills CLI](https://github.com/vercel-labs/skills)。Codex 的加载路径与调用方式见 [OpenAI 官方技能文档](https://learn.chatgpt.com/docs/build-skills)。skills.sh 根据安装遥测提供发现与排名，见 [skills.sh FAQ](https://skills.sh/docs/faq)；目录收录不代表 OpenAI 官方推荐或实用效果验证。

普通咨询不读取维护与测试资料；纯事实查询、翻译、简单偏好选择不走完整决策流程。医疗、法律、财务或紧急专业处置应优先依据现实证据，历史分析不能替代专业判断。

## 当前内容

- 十张历史决策案例卡、一张正式对照卡；`reviewed` 限于所列模板和材料审阅，不表示史实独立确证。
- 五张现代方法卡，以及历史推理、学习实践和四案例桥接指南；按需加载。
- 十张现代书籍参考卡，继续保持 `draft`。

本版本保留2026-10-06本地接入后的产品原字节；部分状态文字保留当时的“待收尾复核”，此后指定范围的本地收尾审阅已完成，报告未公开。内容及指定模型行为审阅尚未证明相对普通回答的实用增益、学习效果或现实决策效果；比较测评是后续工作。

## 发布范围与资料限制

公开仓库只含41份技能产品文件和本README、忽略规则。审核报告、验收资料、原始史料与第三方PDF／DOCX／HTML，以及模型运行档案均保留在维护者本地，未公开。

产品中的部分原材料和维护追溯链接因此在公开仓库不可打开；保留链接仅用于说明原核读位置。GitHub网页也不支持本地编辑器的`:行号`定位格式。使用卡片摘要与在线出处时应遵守卡内证据边界；需要回读本地原文时，先取得对应版本并核对定位。未取得原材料，不能宣称已独立复核。**公开仓库不是完整验收档案。**

本次未指定开源许可证；不为第三方来源新增授权声明。
