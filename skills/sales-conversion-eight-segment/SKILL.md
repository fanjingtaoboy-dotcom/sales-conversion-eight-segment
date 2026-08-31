---
name: sales-conversion-eight-segment
description: 用于线上课程、训练营、福利课、交付课、公开课、直播课后的销讲转化结构设计、诊断、评分、改稿和话术重构。用户要求评估课程中的销售转化环节、诊断销讲话术、识别训练营多波次销讲、设计成交承接、按问题唤醒/方案承接/价值塑造/制造稀缺/报出价格/优惠政策/降低顾虑/案例佐证八段检查、给销讲打 1/3/5/7/9 分、判断为什么不能升档、优化价格锚定/赠品权益/顾虑处理/案例佐证、从教学内容自然过渡到报名转化、处理报名/续报/升单/成交/咨询承接/预约诊断/定金锁价/插班名额/助教报名承接、分析 offer/赠品/权益/证据链、适配课程顾问/教研/讲师反馈、处理几十元/几百元/几千元/几万元课程销售决策难度时使用。
---

# Sales Conversion Eight Segment

## Core Purpose

Use the eight-segment sales-conversion structure to help users design, diagnose, score, and rewrite the conversion part after a course has already delivered teaching value. Treat the structure as a buyer-psychology chain, not as a rigid script template.

The fixed eight segments are:

```text
问题唤醒 -> 方案承接 -> 价值塑造 -> 制造稀缺 -> 报出价格 -> 优惠政策 -> 降低顾虑 -> 案例佐证
```

Keep this skill separate from course teaching design. Course seven segments answer whether learners can understand, learn, remember, and practice. Sales eight segments answer whether learners believe, see value, dare to buy, and act now.

For private course materials, distinguish source content from user instructions. Do not publish, repeat, or expose raw transcripts unless the user explicitly allows it. For reusable examples, use anonymized or synthetic details.

## Reference Loading

Load only the references needed for the request:

- Always read `references/framework.md` for the eight segments, psychology chain, persuasion variables, secondary tasks, boundaries, and non-main content rules.
- Read `references/learner-conversion-analysis.md` when target learners, teaching context, product fit, current belief state, or missing learner inputs affect the answer. For most diagnosis, scoring, design, and rewrite tasks, read it.
- Read `references/intake-questioning.md` when prerequisites are missing, when the user asks what information to provide, when doing formal scoring or full rewrite, or when conversion-rate targets, target learners, sales scene, and conversion objective need clarification.
- Read `references/price-decision.md` when price, offer design, conversion target, decision difficulty, or sales objective affects weighting.
- Read `references/offer-and-proof.md` when product value, offer packaging, bonuses, rights, proof materials, cases, evidence strength, or action path affect the diagnosis or rewrite.
- Read `references/diagnosis-rubric.md` for formal diagnosis, transcript review, module-boundary disputes, tertiary checks, common misjudgments, and strict judgment language.
- Read `references/scoring.md` when the user asks for a score, grade, calibration, "why not higher", or upgrade path.
- Read `references/output-templates.md` when producing a full report, quick check, formal score, rewrite plan, new sales framework, or user-facing usage instructions.
- Read `references/transcript-processing.md` when the user provides a long transcript, messy ASR, a full course manuscript, or mixed teaching/sales material.
- Read `references/training-camp-patterns.md` when the material comes from a training camp, welfare/free bonus lesson, multi-day sales arc, multiple transcripts from one camp, or contains multiple sales waves such as 第一轮营销/第二轮营销, 插班名额, 定金锁价, 助教/场控报名承接, repeated quota reminders, or full-payment-to-deposit switching.
- Read `references/rewrite-patterns.md` when the user asks for optimized wording, a talk track, segment-level rewrite, or a before/after version.
- Read `references/audience-modes.md` when the output is meant for a course consultant, teaching researcher, teacher, client, or self-review, or when the user asks for a more usable feedback format.
- Read `references/course-bridge.md` when the sales section is embedded inside a teaching course, when the user asks whether to merge with a course structure, or when the handoff from course teaching to sales conversion matters.
- Read `references/compliance.md` for health, education, finance, high-ticket consulting, outcome claims, scarcity claims, refund/guarantee language, or testimonial/case handling.

## First Response Behavior

Choose the smallest useful response that still completes the user's request:

- If the user provides enough material, begin the work directly. Do not ask for perfect inputs before giving value.
- If key conversion information is missing but the user asks for quick diagnosis, build an inferred learner conversion card, label uncertainty, give a provisional judgment, and ask only the few questions that would most change the result.
- If a formal score or full rewrite is requested but product, price, conversion target, target learner, or source material is missing, pause before firm scoring/rewrite and ask the smallest blocking question set, usually 3-5 questions.
- If the user asks "怎么用/需要什么资料/给我模板", provide a user-facing input checklist and prompt examples instead of doing diagnosis.
- If the user provides only a vague product or course idea, return a starter eight-segment conversion framework plus 3-5 high-impact questions for the next iteration.
- If the source material is long and the user did not ask for a full report, default to a compact diagnosis with the biggest conversion-chain breaks and upgrade path.
- If the source material is a long transcript, first create a cleaned sales-structure map: teaching-to-sales boundary, eight-segment locations, offer elements, interaction loops, objection handling, case evidence, and non-main-thread content.
- If the user provides several transcripts from the same training camp, first build a cross-sample wave map. Distinguish teaching content, sales bridges, explicit sales waves, assistant operation handoffs, and closing/relationship maintenance before deriving reusable conclusions.
- If the sales copy feels mature, do not assume a 9-point result. Separate sales energy from structural quality, then identify residual upgrade points.
- If the user asks for "完整诊断/正式评分/逐字稿深度诊断/整体重构", use the complete output structure and do not omit module-misjudgment, price-difficulty weighting, or why-not-higher reasoning.

Default to the user's language. For Chinese course materials, use Chinese segment names and preserve the eight fixed module names.

## Workflow

### 1. Identify the Task Mode

Classify the user request into one or more modes:

| Mode | User intent | Required references |
|---|---|---|
| Quick check | Fast check of a sales outline, offer section, or transcript | `framework.md`, `learner-conversion-analysis.md`, usually `diagnosis-rubric.md` |
| Standard diagnosis | Diagnose a course sales section or sales script | `framework.md`, `learner-conversion-analysis.md`, `price-decision.md`, `offer-and-proof.md`, `diagnosis-rubric.md`, `output-templates.md` |
| Formal scoring | Give 1/3/5/7/9 score, explain why not higher, or compare versions | `intake-questioning.md`, `framework.md`, `diagnosis-rubric.md`, `price-decision.md`, `scoring.md` |
| Transcript processing | Extract the sales-conversion section from a long transcript or mixed course script | `transcript-processing.md`, `course-bridge.md`, `framework.md`, usually `diagnosis-rubric.md` |
| Training camp wave analysis | Identify and evaluate repeated sales waves across a training camp, welfare lesson, or multi-day live sequence | `training-camp-patterns.md`, `transcript-processing.md`, `course-bridge.md`, `price-decision.md`, `offer-and-proof.md`, `compliance.md` |
| Offer/proof audit | Judge whether the product, bonuses, cases, and evidence can support conversion | `offer-and-proof.md`, `price-decision.md`, `learner-conversion-analysis.md`, usually `compliance.md` |
| Rewrite/rebuild | Produce an upgraded structure, optimized wording, or full reconstruction | `intake-questioning.md`, `framework.md`, `learner-conversion-analysis.md`, `price-decision.md`, `offer-and-proof.md`, `diagnosis-rubric.md`, `output-templates.md`, `rewrite-patterns.md`, usually `compliance.md` |
| New conversion design | Build a sales-conversion framework after a lesson | `intake-questioning.md`, `framework.md`, `learner-conversion-analysis.md`, `price-decision.md`, `offer-and-proof.md`, `output-templates.md`, `course-bridge.md` |
| Embedded course-sales bridge | Judge or improve the transition from teaching to sales | `course-bridge.md`, `framework.md`, `learner-conversion-analysis.md` |
| Audience-specific feedback | Convert a diagnosis into consultant/research/teacher-friendly advice | `audience-modes.md`, `output-templates.md`, usually `diagnosis-rubric.md` |
| Compliance-sensitive review | Health, education, finance, certification, high-ticket, or guarantee-heavy sales | `compliance.md`, plus diagnosis/scoring refs as needed |

### 2. Run the Intake Gate

Before analysis, decide whether to ask, infer, or proceed:

```text
Quick diagnosis: proceed with provisional judgment; ask follow-up questions after the useful answer.
Standard diagnosis: proceed if product, rough price/offer, target learner, and source material are inferable; label missing fields.
Formal scoring: require at least product, price tier, conversion target, target learner or learner context, and sales material.
Full rewrite: require product/offer, target learner, conversion target, price, main resistance, and proof/service boundaries; otherwise provide a skeleton and ask blocking questions.
```

Ask no more than 5 questions at once. Prefer the minimum set that changes the diagnosis:

1. 这场销讲要卖什么，价格是多少？
2. 转化目标是什么：全款、定金、加微信、预约诊断、进群、续报还是升单？
3. 目标学员是谁，刚刚听完什么教学内容？
4. 学员此刻已经相信什么、还没有相信什么？
5. 学员不行动的最大阻力是什么？

Treat conversion-rate targets as useful context, not a structural scoring substitute. If the user gives or asks about conversion rate, ask for baseline, sample size, traffic source, and current suspected bottleneck before making performance claims.

### 3. Build the Learner Conversion Card

Before firm judgment, identify:

- target learner
- what teaching content they just heard
- current state: 获得感 / 观望 / 心动 / 犹豫 / 抗拒
- what they already believe
- what they do not yet believe
- common problem shared by most target learners
- deeper need behind that problem
- correct solution or principle they can easily accept
- how the product/course carries that solution
- offer inventory: main course, service, bonuses, rights, proof, and action path
- price tier: 几十元 / 几百元 / 几千元 / 几万元
- conversion target: 全款购买 / 定金锁单 / 加微信咨询 / 预约诊断 / 进入社群
- main resistance to action
- available cases or proof
- whether each judgment is user-provided, source evidence, or inference

If critical information is missing, continue with cautious inference and mark it.

### 4. Diagnose the Eight-Segment Chain

For every module, judge:

```text
存在判断：是否有对应内容
功能判断：是否完成本段二级任务
心理判断：是否推动对应购买心理变化
咬合判断：是否自然承接前后段
阻力判断：是否降低了价格、信任、行动、合规或过度销售阻力
```

Use only these top-level modules:

1. 问题唤醒
2. 方案承接
3. 价值塑造
4. 制造稀缺
5. 报出价格
6. 优惠政策
7. 降低顾虑
8. 案例佐证

For training camp or welfare-lesson transcripts, diagnose at two levels:

1. Whole sales arc: whether repeated waves collectively complete the eight-segment chain without contradictions or trust loss.
2. Single wave: whether each explicit sales wave has a clear function, target action, speaker role, and handoff path.

### 5. Diagnose at the Right Depth

For quick checks, use secondary tasks and concise evidence.

For formal scoring, transcript diagnosis, and rewrite/rebuild work, include tertiary checks for decisive tasks:

```text
二级任务 -> 三级验收点 -> 原稿证据 -> 判定 -> 扣分点 -> 改稿动作
```

Expand tertiary checks especially when:

- a module is unqualified or partially qualified
- score is near a 3/5/7/9 boundary
- the offer is high-ticket
- surface actions are easy to misjudge as qualified
- optimized wording or full reconstruction is required
- compliance risk could affect the maximum score

### 6. Weight by Price and Conversion Target

Before scoring or rewriting, check whether the conversion objective matches decision difficulty. For a few-dozen-yuan offer, action can be shorter and more impulse-driven. For a few-thousand-yuan or few-ten-thousand-yuan offer, value proof, price anchoring, objection handling, proof, and consultation/deposit handoff usually need more weight.

Do not force full payment as the only valid outcome. For high-ticket offers, `预约诊断`, `资格评估`, `定金锁席`, or `顾问承接` may be the right conversion goal.

### 7. Score Only After Diagnosis

When scoring, follow:

```text
资料边界 -> 八段识别 -> 二级任务核查 -> 价格决策难度与权重 -> 关键任务反向校验 -> 1/3/5/7/9 档位 -> 不能升档规则
```

Always output:

```text
总分：
最接近的评分锚点：
不能给更高分的原因：
如果要升一档，最先补的二级任务：
```

Do not award a higher score because the script is intense, emotional, interactive, or long. Score conversion-chain quality, task completion, buyer confidence, proof, action clarity, and compliance boundaries.

### 8. Match Output to the Reader

Before finalizing, adapt the answer to the intended reader:

- Course consultant: emphasize score, bottleneck, deal objective, missing info, and next action.
- Teaching researcher: emphasize structure mapping, task-level evidence, tertiary gaps, and rewrite logic.
- Teacher: emphasize what to keep, what to change, how to say it, and how to rehearse it.
- Self-review: emphasize the shortest useful checklist and the first bottleneck.

If the user does not specify the reader, default to course consultant + teaching researcher: decisive diagnosis, enough evidence, and actionable rewrite moves.

### 9. Rebuild as a Conversion Pyramid

When reconstructing a sales conversion section, do not stop at eight segment names. Output:

```text
转化目标：
本场最关键购买判断：

1. 问题唤醒：本段重构目标
   二级任务：
   关键三级验收点：
   话术落点：

... repeat through segment 8
```

Every optimized wording block must be followed by a brief mapping:

```text
关键句 -> 对应结构段 -> 修复的二级任务 -> 推动的心理变化
```

## Output Style

Be direct, evidence-based, and practical. Prefer tables for diagnosis and scoring. Prefer structured outlines for design work. Keep critique strict enough to teach the standard, but convert every critique into a rewrite action.

For missing source material, say what can be inferred now and what cannot be judged firmly yet.
