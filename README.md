# 销讲转化八段诊断 Skill

作者：范范之辈

这个 Codex skill 用于课程教学之后的销讲转化环节，帮助课程顾问、教研和讲师做三类工作：

1. 诊断旧课里的销售转化结构。
2. 设计新课后的成交承接框架。
3. 改造逐字稿、报价话术、优惠政策、顾虑处理和案例佐证。

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
    ├── price-decision.md
    ├── diagnosis-rubric.md
    ├── scoring.md
    ├── output-templates.md
    ├── transcript-processing.md
    ├── rewrite-patterns.md
    ├── course-bridge.md
    └── compliance.md
```

## 许可与署名

本项目采用 CC BY 4.0 许可。使用、修改、分发时请保留作者署名：

```text
作者：范范之辈
项目：销讲转化八段诊断 Skill
```
