# 销讲转化八段诊断 Skill

作者：范范之辈

这个 Codex skill 用于课程教学之后的销讲转化环节，帮助课程顾问、教研和讲师做三类工作：

1. 诊断旧课里的销售转化结构。
2. 设计新课后的成交承接框架。
3. 改造逐字稿、报价话术、优惠政策、顾虑处理和案例佐证。

也支持训练营/福利课里的多波次销讲识别，例如：第一轮全款成交、第二轮定金锁价、插班名额、助教报名承接、报名播报、课后作业收束等。

新版本额外强化了“0元表单/免费营/结缘营用户转近3000元或几千元系统班”的判断：会先检查用户热度、免费体验获得感、信任缺口、服务系统、风险逆转、证据矩阵和高客单行动路径，避免把高客单销讲误判成普通低价福利课。

核心结构：

```text
问题唤醒 -> 方案承接 -> 价值塑造 -> 制造稀缺 -> 报出价格 -> 优惠政策 -> 降低顾虑 -> 案例佐证
```

它和“课程七段结构”是互补关系：七段解决学员是否听懂、学会、记住、愿意练习；八段解决学员是否相信、觉得值、敢买、现在行动。

## 安装

下载本仓库后，把 `skills/sales-conversion-eight-segment` 放到你的 Codex skills 目录：

```bash
mkdir -p ~/.codex/skills
cp -R skills/sales-conversion-eight-segment ~/.codex/skills/
```

重启或刷新 Codex 后，使用 `$sales-conversion-eight-segment` 调用。

## 怎么用

你可以这样提问：

```text
使用 $sales-conversion-eight-segment，帮我诊断这段课程销讲逐字稿，按 1/3/5/7/9 打分，并说明为什么不能更高。
```

```text
使用 $sales-conversion-eight-segment，基于这节交付课内容，设计后半段销售转化结构，目标是预约诊断。
```

```text
使用 $sales-conversion-eight-segment，帮我把这段报价和优惠政策改得更清楚，注意不要用虚假稀缺和绝对承诺。
```

```text
使用 $sales-conversion-eight-segment，帮我检查这个 offer、赠品、案例和报名路径是否足够支撑 2999 元课程转化。
```

```text
使用 $sales-conversion-eight-segment，这几份稿来自同一个训练营。请先识别每节课里的销讲波次，再提炼哪些模式值得沉淀成可复用规则。
```

```text
使用 $sales-conversion-eight-segment，这是一批0元表单用户听完免费营后转近3000元系统班的逐字稿。请先识别销讲部分，再判断免费体验、信任加热、offer服务系统、风险逆转和案例证据是否足够支撑高客单转化。
```

## 最小前提

如果想让诊断更准，建议先提供 5 个前提：

```text
1. 这场销讲要卖什么，价格是多少？
2. 转化目标是什么：全款、定金、加微信、预约诊断、进群、续报还是升单？
3. 目标学员是谁，刚刚听完什么教学内容？
4. 学员此刻已经相信什么、还没有相信什么？
5. 学员不行动的最大阻力是什么？
```

如果是 0元表单/免费营/结缘营转高客单，建议额外补充：

```text
入口来源：
免费体验深度：听课天数 / 作业 / 实操反馈 / 互动 / 是否加微信
已建立信任：
尚未建立信任：
售后/退款/保障规则：
可脱敏案例素材：
```

如果只是快速诊断，不提供完整信息也可以；skill 会先给暂判，并标注哪些判断来自推断。

转化率目标可以补充，但不建议单独作为诊断依据。更好的写法是：历史转化率、目标转化率、样本量、流量来源，以及你怀疑卡在“听不下去、觉得不值、不敢买、不知道怎么行动”哪一步。

## 最好提供的资料

```text
课程主题：
目标学员：
刚刚交付的教学内容：
销售产品/课程：
课程价格：
优惠政策：
赠品/权益：
转化目标：全款 / 定金 / 咨询 / 预约 / 入群
直播/课程场景：训练营单课 / 交付课 / 公开课 / 专题课
学员当前状态：获得感 / 观望 / 心动 / 犹豫 / 抗拒
学员主要顾虑：
成功案例素材：
报名路径：
合规限制：
已有材料：大纲 / PPT / 逐字稿 / 录音转写 / 其他
希望输出：快速诊断 / 完整诊断 / 评分 / 重构方案 / 优化话术 / 新销讲框架
```

资料不完整也可以使用，skill 会先做谨慎推断，并标注哪些判断来自推断。

## 仓库结构

```text
skills/sales-conversion-eight-segment/
├── SKILL.md
├── agents/openai.yaml
└── references/
    ├── framework.md
    ├── learner-conversion-analysis.md
    ├── intake-questioning.md
    ├── offer-and-proof.md
    ├── price-decision.md
    ├── diagnosis-rubric.md
    ├── scoring.md
    ├── output-templates.md
    ├── transcript-processing.md
    ├── training-camp-patterns.md
    ├── lead-form-high-ticket.md
    ├── rewrite-patterns.md
    ├── audience-modes.md
    ├── course-bridge.md
    └── compliance.md
```

## 迭代与评测

这个仓库包含一套轻量评测材料，方便持续优化：

- `evals/test-prompts.md`：基础测试提示。
- `evals/golden-cases.md`：1/3/5/7 分、价格错配、合规风险等黄金样例。
- `evals/regression-checklist.md`：每次更新后的回归检查清单。
- `docs/iteration-playbook.md`：如何把真实使用反馈沉淀成下一轮规则。

提交反馈时请先脱敏，不要上传真实姓名、电话、微信、订单、未授权学员案例或完整私密逐字稿。

## 许可与署名

本项目采用 CC BY 4.0 许可。使用、修改、分发时请保留作者署名：

```text
作者：范范之辈
项目：销讲转化八段诊断 Skill
```
